<template>
    <section class="pdf-content">
        <section class="report-info">
            <section class="image-container">
                // <img
                //     class="user-image"
                //     :src="require('@/assets/axe.jpg')"
                //     alt="User Image"
				// 	ref="userImage"
                // >
            </section>

            <section class="user-details">
                <h4 class="user-name">
                    Mogul Khan Touch This
                </h4>

                <span class="detail-container">
                    <span class="detail-label">
						Game:
                    </span>

                    Game No. 3
                </span>

                <span class="detail-container" >
                    <span class="detail-label">
						Date and Time
                    </span>

					November 11, 2019 1:00 PM - 2:23 PM
                </span>
            </section>
        </section>
    </section>
</template>

<script>
export default {
    data () {
		return {
			series: [
				{
					name: 'Level',
					data: [
                        { y: 1, x: '11/11/2019 13:00:00' },
                        { y: 1, x: '11/11/2019 13:01:00' },
                        { y: 2, x: '11/11/2019 13:02:00' },
                        { y: 4, x: '11/11/2019 13:03:00' },
                        { y: 5, x: '11/11/2019 14:04:00' },
                    ]
				}, 
				{
					name: 'Experience',
					data: [
                        { y: 5, x: '11/11/2019 13:00:00' },
                        { y: 5, x: '11/11/2019 13:01:00' },
                        { y: 10, x: '11/11/2019 13:02:00' },
                        { y: 12, x: '11/11/2019 13:03:00' },
                        { y: 20, x: '11/11/2019 14:04:00' },
                    ]
				},
				{
					name: 'Gold',
					data: [
                        { y: 10, x: '11/11/2019 13:00:00' },
                        { y: 10, x: '11/11/2019 13:01:00' },
                        { y: 20, x: '11/11/2019 13:02:00' },
                        { y: 30, x: '11/11/2019 13:03:00' },
                        { y: 50, x: '11/11/2019 14:04:00' },
                    ]
				}
            ],
            
			chartOptions: {
				dataLabels: {
                    enabled: false,
                    
					style: {
						colors: ['#fff']
					}
                },
                
				stroke: {
					curve: 'smooth'
                },
                
				chart: {
					toolbar: {
                        show: false,
                        
						tools: {
							download: false,
						},
                    },
                    
                    animations: {
                        enabled: false,

                        animateGradually: {
                            enabled: false
                        },

                        dynamicAnimation: {
                            enabled: false
                        }
                    },
                },
                
				tooltip: {
					enabled: true,
					// theme: true,
					x: {
						show: true,
						format: 'MMM dd, yyyy HH:mm'
					},
                },
                
				legend: {
					show: true,
					labels: {
						useSeriesColors: false
					},
					onItemClick: {
						toggleDataSeries: false
					},
					onItemHover: {
						highlightDataSeries: true
					},
                },
                
				xaxis: {
					labels: {
						style: {
							// colors: '#fff',
                        }
                    },
                    
					type: 'datetime'
                },
                
				yaxis: {
					labels: {
						style: {
							// color: '#fff',
                        },
                        
						formatter: (value) => {
							return value
						},
                    },
                    
					type: 'text'
				}
			}
		}
    },
    
    mounted () {
		this.$nextTick(() => {
            setTimeout(() => {
                this.$emit('domRendered')
            }, 1000);
		})
	},
}
</script>